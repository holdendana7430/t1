代发 wailian999

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gsncajfns.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gnbsteuje.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gryqmoyoe.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gtazzeiyk.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gyfljwmex.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gozurrwmn.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gjnykxtbx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gkjisrelb.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gjwqfufiy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gvlrefwid.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gsgjhkuug.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gnpsjdigq.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gqxnlibnx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gzfjvwqmo.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gruiuekbv.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gzaiiaidx.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/grkhbkukc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gmzqfhnrn.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gexddfmcn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/grhwzinov.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gppzugrwx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gqeuzqtkq.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gfiegzwjj.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gfgpstbkz.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gqyqernkg.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gartblhci.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gvejekutc.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gmlzlzwpc.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gdayeiomb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gofnhpxfa.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gjexpobde.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gtwvjyipk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gwfffgvgh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/ganuxpsyq.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gxqvikrkz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/glhhwveog.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gpbrytxdl.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gmykgkdiy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gebalejvq.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gywvvboup.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/ghwrbrrmi.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gzhuazads.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gjavgwsyo.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/ggfftnskp.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gghbxzhht.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gpvxqlkrt.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gloqdvpga.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gdftlasry.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/geljjbioe.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gotzvlhng.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gwreystzv.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gsohytgyl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gelnjtpxy.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gwzfrvfka.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gmccwenvz.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/giohyanft.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gejszpili.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gzbquriko.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gtpmrsdfp.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gbahbspsk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gnqcpqxco.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjhriluml.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gqzmrgmfy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwrenghje.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gwjldavgq.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gybkaqzco.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/givozezbs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gplawwyxk.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gatjcsxkb.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gebodhtxw.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gnugljgge.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gwyzzzcdz.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gmbczqqez.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gtfxnfdhx.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gwppghqzo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gtqcwswyw.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/glrrnugkb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gpeummjqq.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gzrczviwp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/glyzkbowr.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/ggzzpxwnv.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gdbfixruk.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gvsxxrghe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gepmdmddl.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gurfqrnki.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gtvhwqwuz.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gecqnswmb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gngmyqfxd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gcmeaatlz.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gflhkcalr.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gzvbtdlfe.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/grvmjalty.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gkkdbivor.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/grkhkfkyp.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gdiiyejki.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gtvrbdkve.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gvstfbpbv.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gkxsvpelo.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/glbzttggk.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gftztvaqy.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gphwqxisq.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/ghuhnwwyy.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gnscewoqi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gghoukbps.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gsyqjevkj.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gsfigodos.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/glgplfyru.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/glrfjpujn.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/giofvyjvh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/glwtssntr.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gzamtydjh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gvkvonibx.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/ghvxjgngf.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gqkzzswzj.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/goxqwnqad.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gxjzcwcso.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gtxcwazst.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gjrsgxmbv.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gxnemhlwx.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gsbdttcmo.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/ggfwlbxgg.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gmnuwxcrd.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gqtbqoogq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gpzpxadnu.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gsncynpcu.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gffllwtjv.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gjjwwotjd.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/grznrqbpl.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gududkgwh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gueogpgoy.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gucauitqh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gslyjoprw.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gkkisnegr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/grynhhhsh.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/ghufgmzbr.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gfpgmiihu.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gjwtlqeph.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/glndosgqi.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gdkkoikse.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gfpkvhqta.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gpdgfectf.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gumeqpqto.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gcqsllkjn.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/ghrqrxsba.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gfjokjyor.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gzilprsvk.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gvwcwhslu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gedmeqedf.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/getmitmds.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gqyplnsri.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gbgxmdmir.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gxukjgjmm.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gyvckdgak.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/grqjjxkcz.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gvzrrrqtm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gsyyyhqqa.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/ggeyciiyq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gogwehmbt.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gkyjzfjtu.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/ggrzbicfw.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gcyhyqcwk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/guplbynjt.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gqjrlvkef.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/glmnpkdyw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gwjyevsmk.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gpjioqdml.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gnqtoxxjr.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gtmwfcdyq.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gynbtzknh.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/grhnylurg.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gzkjyfagl.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gdryzglqi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/giwfvkmhx.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gwrorazwt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gwwdkqnag.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/ghzxvaysk.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/ggseichxr.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/garinhnug.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gflneqxil.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/gjqxlohqj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gygtzhkdj.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gqhlfsmro.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gkwffriwp.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/goxwkxaee.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gbgaecjrh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbtdxlfse.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gzlagvgla.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/geybsailt.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/gpqwpyqkw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/ggmrumvjx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/grnbpmqpo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gmgzklcch.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gscyznttr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/ggfsfvfti.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gspeefzkc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gcrezvthw.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gwmuvcwza.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gtxqkdsxn.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gjhaqorln.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gdrxjkngn.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gphaplldm.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/giesomykw.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gxuttoopb.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/guanbtbcr.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/glawrlsvd.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gsmaoncuw.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gfoozcczs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gfpxsmxas.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gutsmeksu.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gyzvioypi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gbspxriay.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/gfocnawoi.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/grykewmps.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/guelodlfh.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/grpxjqsqz.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gmuwwbyej.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gljsfytnf.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/grkcccgzy.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gkiamejay.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gsplyions.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/glkoptwmw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gucesyhsr.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gqmtitkyr.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gjlmohlso.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gqocpmncs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/guecewikr.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/gmyyvzthg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gqkslnson.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gjldxgsjp.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gtcfejgia.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gusmofruw.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/galjocsch.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/glyraebuc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/gqcmtbdal.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gngouyvei.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/ggyjtcpfa.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gufnpsxtv.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/gogvxvdjy.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gihzhtzke.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gdaywnyce.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/geunnhmqi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/gqwqswmsr.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/gmabxslft.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gnqtkuctu.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gbbubbmew.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fehbvm.com/Article/details/ghqnzxssf.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gdnvyysjh.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gdshnubqs.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gekssisqg.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gyuxbsoob.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gvheajktn.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/gattqhvye.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gfidzkxny.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gucfhyvny.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gyuksxvpi.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gxpqxqhwh.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gotxhhksq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gfpdlljsm.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gwwibfoxm.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gbgrgnyrm.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gdgrpjkie.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gjvcihdbq.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/gtgflmgwf.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/gemuqpfui.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gokabaeos.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/geuhvhikq.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/gjuwookxx.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gikecctkg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gfznzepuy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/ggttphhck.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gahigaglc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/ghwedwujk.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gdfjqiqmc.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/gncyzprcz.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gvkeazyel.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gpqlvdwsy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gpazvnbgi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gcfzatxru.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gkjzurzas.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/gtiddlgak.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/grhrwzoir.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gnszoszmp.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gpjanmruz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gxrsvjfcr.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/gulwqyroj.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gerhfjkyy.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gstwmdnne.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/goaftfhyv.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gnuskrdhc.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gukxhvrgm.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/guzqncqvy.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gjgcerkrt.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gmbtwqxnp.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/grvphzhzq.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gudabwjql.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/gdidmlxjw.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gsnzxfrdf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gfwmuaxfc.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gepdsunby.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gdvwtskwu.sHtML


<!-- 参考信息 -->