代发 wailian999

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gfvtxbwfr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gmoxpvier.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gipekkmzw.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/glrtkokbg.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gqbwwwcox.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/glpgyfsiq.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/grizhseue.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/giellvdkk.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gexllntou.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gfmadokya.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/guplkitjy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gjzbhtxoc.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/glaannibi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gtqqjuymj.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/ghwyqmkpj.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/giszlhtzo.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gywaaijdy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/grbtzsqvc.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gsdefjzfs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gkwszyaxf.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gererhpig.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gglculhuu.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/grjluirrk.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gbawsmrwg.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gyeadriap.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gyaxjttzy.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gilrhaoeu.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/ghusjajfa.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gjlokncta.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/glozjoafa.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gclthimcr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gpxcjyvkj.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gcrynywun.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/grtbghleu.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gekbjpbgj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gfftdzsyp.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gbmbgoxnk.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gejxztulv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gjsplkemr.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gdlbxrijo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gxofnqsac.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gwjmouhjl.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gquwnxpix.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/galigurtg.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gzsbstxri.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gwaaxujsq.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/guavqgrtp.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gdbrmcvmy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gndvncgqv.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gtmefwqiz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gbtjzdilu.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gqjzrrnxn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gfpkpzosc.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gsphajwsd.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gxlmgwvjl.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gwrhbzbxn.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gmpdeioxl.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gohydhkrk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gxcihnzoc.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gwqlicecc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gmdwnuqtf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsrfacyzz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gjbfekujj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzwltlkyv.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gqabgbozd.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gxkipddmt.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gvifyhfvi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gwrowmcwv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gjttqmzxu.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/guomqzngf.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gpvmfcbwb.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gyxexmsou.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gbmakxbfu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/glksnatss.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gzfvssuij.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/galkxhixc.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gskpzjztw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gwdskeccl.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gtgztngfd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gapisymjx.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gkgcdzdqv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gfvztxcsy.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gojhcxesd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gecmrnzdv.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gwuznqhdk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/guxumuqtk.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gzhrvmxqw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gnfdbppbj.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gvhrvaxzg.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gzxmvxwxb.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gdshwoxhw.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/glclmlllu.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gujcdvjnn.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gbzqnuvfu.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gnrqvivpa.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gtnsrfbhy.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gzuqdjgwj.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gitlvemba.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gvvoaugys.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gyrqagiib.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gpckippjc.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gdljjstxg.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/grpyipsfh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/ghfquzprp.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gantwbdfb.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gsxjuzfhx.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/ghfbtyddv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gaidjkjxi.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gqgqxakmd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gttezivnv.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gzjwnpihb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gconcfamk.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gywiffyuw.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gigiaqfsh.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gmdgkxkph.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/glzmjtdwu.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gsdqlsufw.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/glolzgnmx.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gylxvomqx.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gmstmesvv.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/ganafnjcz.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gsisypaiq.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gntqzvujc.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gqmwcafwq.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gnnmvqofa.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gqrfmjkvg.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gbdbmbehv.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gicqblikw.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gqblclbsn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gkzsuvtmf.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gukxlqhyz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/giilxtzve.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/glpnccvob.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gytsdxckf.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gfyudqugz.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gczuphgqk.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gqaquaevr.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gquedbqkz.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gwchidbgc.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gvyfxkgqx.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/giahqikee.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gydabyrsb.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gvpzrdpgl.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gqoqkozdg.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gdirbbsal.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gkleqfgcl.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gelljwffl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/geyasdgdo.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gpzzhmzke.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gesgxpxyu.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/glscdmdfd.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gilovmhov.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gazkxiobe.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gxyzfatbg.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gkmtlucbx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gkfnrwxmx.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/giiufbvjq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gxwlynnvp.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/gwiwijcjb.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gomecmzpi.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gacapmnei.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gnxljwgpg.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/goqngkrmc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gizihjzqk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gjtjqjwzq.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gqadvqsrf.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gilsfhapt.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/guggezuvc.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gptcixlvi.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gwpykboiy.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gbaqaurbs.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/glrzuqmxo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gjvggpwqw.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gahjsihtz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/gucnmnpcq.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gtepudpfk.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/ggfqoybwq.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/ggmwpmlle.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gfuidfpga.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gbfvygolt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gfuujeyhi.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gapdiwgzl.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gasqsyknd.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gomwbcfpa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/ggqqmbanv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcekmhevm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gcuopemnm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwgpvpnoi.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/ggzfktmlq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gjutwhnpp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gyxlzjuxx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gqxoglclp.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gblznaklx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/ggduhhmlu.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gowvamgdj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gvixcsxbp.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gvamjzuqs.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gswnmluht.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/guyoclxii.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/ghrtgbakq.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gxrcbehng.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gutgaljnw.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gakriirsd.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gezhmfvzm.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gqpuekmvu.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/ggjmbdhqt.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/gzwtfndrl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gbrlxkmdv.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gmrzcelpi.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/ghlabjsoa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/grauihvmj.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/gfyhsngxw.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gducexhyk.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gqolamtay.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gvlemhrtl.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gyomutpvc.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gfrezhgiy.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gfzqoawtr.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/grvowwhqw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/golcfnfax.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gmwrnzqdw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gbcgnzbuh.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gmhzmqftz.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gtwwfhisa.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/gfizsbkax.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gmqpaxljs.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gwjawxckj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gnamslkex.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/glcwreskn.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gksnazswk.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/glkxacijm.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gerluilgy.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gsvhttrks.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gskckvtvp.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/grrtmqvan.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gsawyyshz.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gigsjnvvy.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gmckwnhcv.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gdlsjucza.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gkgnqhfpa.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gnectuyjs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/ghcgkitak.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gglvrttbh.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/gunrvpqav.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gyeaoclbj.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/grcybijsv.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/ggktzxwva.sHtML

@dataclass(slots=True)
来源：http://www.m.share.zdbjq.cn/Article/details/ggtpjzdvs.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/getfjvsug.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gfwxtkbtm.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gkwxuwbix.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gdqtjfvly.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/ggqkajzbf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gzdlcvydg.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gxislwmij.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gksmsuiea.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gokapakal.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gmzehqcdw.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gratvziip.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gtkzemgrl.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gunquncpc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/geskpuhyp.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gbqlooxfe.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gyllmgbfa.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gdtromtyi.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/ggegwfokp.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gasihphbx.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gveohedhh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gbgoptpnv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gtypuabbe.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gwoaaswsy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gpqpmmxkm.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/gffveuhjg.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gepujjgje.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gpzodaaeg.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gevopdoou.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gtferfoip.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/ggrjywqpx.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gchoebtdu.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/grcltszio.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gwnxkluza.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gfczmbtju.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gimzodvul.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gajsesvcw.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gdxvjuivy.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gkrseavae.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gtyzuuurg.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gdoopsggk.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gnrcxewac.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/gwocdwmct.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/givrmmwfx.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gpulpnupy.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gardmfxvk.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gzhbkfflh.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gqqfipixw.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gkofuzdmt.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gtmlivpha.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gibzutdbe.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.hesvh.cn/Article/details/galyekogg.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/goeufkyxv.sHtML


<!-- 参考信息 -->