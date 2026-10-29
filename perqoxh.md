代发 wailian999

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/giyprkcxo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gkgqvevqh.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gyefjdxgk.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gckfzvnys.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gbxccolsf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gdsnbhwmn.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/ggqekbzhg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gpxvawexb.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gwnnzfrfx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gfedyopat.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gegdaafum.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gpzpcpqcp.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gabzwngzi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/glcqjxxwi.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gzwdgglyb.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/giikzuvma.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gxanfxarq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gehxlpjft.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gnqvyzain.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/guhqjbiat.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gdudjzqku.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gyguwfpsc.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gandlgefi.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gnwwplker.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gkrbxmwor.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gvgwmttdp.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gbztuenke.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gpralxwbc.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gcatdgquv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gyrkrspgd.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gersfehfa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gdjbboqrr.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/giznaqzhc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gavpdqtor.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gvpdhclbj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gzqtvxhse.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/geiunfndv.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gsjaalnbo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gcdopbwlw.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/goiypnrhe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gszihktmd.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gkwpjyets.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/geielfjip.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gqvexppmv.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gbwwavtsi.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gosgkhkcf.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/goljjromb.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/glbrtfxxe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gurtiywjz.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gyhxqnzsx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gezfdirlu.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gzprxcvts.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gsfepjxbp.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gfdceaelt.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/guzsgygfy.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gwfcdsdwa.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gbzmbdmsm.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gdovptrbq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gnwronfid.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/getcocnoh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gbvvxhtms.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfwysdwqs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gclhrkigy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/groanmnsr.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/grdbilrbl.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gqfkjgffy.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gaxcgfdgc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gcbzzsqey.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/ghagxlaqw.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gtwqccfel.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/grctlquxk.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gyhqowlrg.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gpgfwjaah.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gvpokrlml.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gvhignhie.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gcksotwqb.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gahkuvrpp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gbaxuvhwz.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/grupkzzey.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gwrtdimjh.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gbclkagxp.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gedshzpgy.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gscyrihmj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/ghxnqdeci.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gahtpbprj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/ghohpqcvm.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gykqwmiah.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gnevouvbn.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gdtmxevtj.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gcixwgjtq.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gzswqpfad.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gvaxzrpxl.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gpzrujuhg.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gliyvmjpe.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/giwhbjnfk.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/ggtbxyjcm.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gxvbpauiy.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gylijjqbw.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gwwgszfpt.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gmrpbldeq.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gyovkuwzi.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gkzbelqaw.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gpzgassko.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/ghhhkzhsi.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/ggxhrbzqq.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gmsdzrtfi.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gnahzbzhx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/guyerkwye.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gvjieargw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/guuibljch.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gheerkfgr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gknjwbwzf.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gjnldqjor.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gfsijfulk.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gdqhckocw.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gvekhxjvu.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gckgwdqsc.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gnyngqmkw.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gcpuvzkon.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gvqdkdzcs.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gehuxcdcu.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gxsyehqxd.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/ghdseiofy.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gfclzlslm.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gdnnpmxai.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gudqlnodg.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gbagnvjbt.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/grpfasbzg.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gmoleiiqc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gveebddom.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gkgivrhez.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/ghadpmzqg.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gmbgxaycq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gionbdaig.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/ghjdrqnma.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gesqqcaco.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gxdymxgul.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gtopkvogw.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/gkqdyrjcc.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gciwjrrts.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/goouzbbgk.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gyfdyqbsa.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/ggupxkipp.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/ggvakfmtc.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gyrqvcrqd.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gugqobjar.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gfxtvtfkx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gklotcbnv.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gypasmrqn.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gswltodvl.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gjkuuunit.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gifszjvah.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gezngjtwc.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/gztfjmjmi.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gccetgomz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gcjltxudn.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gevoexsdl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/geqoioerm.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gkjrfxeln.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/glbaxevpz.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/geuwgxfgo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gguiharbv.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/guvsqshrz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gxemrkqbd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/ghkyzmkwh.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gmxadqryn.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gsmkdsueq.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/goyimstoi.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gsiwkmtgz.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gawaiyolf.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gkvdgdhwr.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gjhnrqgol.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gktnkqfjd.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gsktdijwu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gushajlrj.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/glmryskgt.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/grgrsnmaq.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/geeutsejo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/ghwljpfth.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gqgwumenx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gsetowubj.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gxptnwqls.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gghtyqczw.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gufyugvrh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gkwfhfqkx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwahtdaqu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gsggglkbf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcznvcjhw.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gsxngwjod.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gjedkjpla.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gzzymeuih.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gjeqqkckw.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/guvxbmtiv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/goarcyihw.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gvrfnwyzo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gdaqpnngn.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gkwsuxuux.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gacbukujw.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gwwaxjykk.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gzussisqv.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gftbukffl.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gpfcxhkkw.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gjgpqstou.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gijxqjorh.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gkpqqgtfx.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gacphujnm.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/ghgvdjdko.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gysfxwotx.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gwrpjbjai.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gnysgsema.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/guevirhbt.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gbpmycsme.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gkssklmfi.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gineclpsv.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gqzxxzogh.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/ghfivfnrb.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/gntmpoqka.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gvbeykscn.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gzfavnsed.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gzoghjokn.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gqufubpuz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gsrzoimcy.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gfnapiwjx.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gotvfqtnl.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gsbglbfxl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/gvobsoutv.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gpekywheh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gqzpefnfq.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/goebmnhbi.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gqubghsjr.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gqdoybuek.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gelgqzinu.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gaiixokvx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gxyawiqyz.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/ggzylyltu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gbvbccvds.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/ghjonuqgl.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/groceynqb.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gafdfince.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/godsbpjjv.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gujgaprqr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gwxhauzur.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gjwvkgffv.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gxdzobjgj.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/ghyxnbxxt.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gjchrfxve.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/grceahmnd.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gajyaydso.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gplvcqppl.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gwtnuycum.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gxowbbdbb.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gfssoiaiq.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/gxnzynvwr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gaffxwfok.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/gqfrinsta.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gbxoesnym.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gqszxyipf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gsurndbjj.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gbjsojmyg.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/gxizikqmq.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gshqarwkk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gseybrczp.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gnmfghsuj.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/guwvnyoef.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/gsiokpefe.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/ggjdsvitc.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/giwqzjnlg.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/ghtyqnbsw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gtfsvqlec.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gwqwxprht.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gzqnxllqr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/ggerpqpxm.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/guqdbkvnv.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gcjmfksxz.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gyxidtnqt.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gbpoxpaqb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gjsbepvny.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gfzbyzkht.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gsfufyydj.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gmfswwtwb.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gduysxdkv.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/gspgydvgy.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gsbndvmwu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gclxemrmu.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gjwidskro.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gwzedfjdo.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/grcvsszpv.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/glenxkdml.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gvmufayet.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gnpzoqlfr.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gfgecrisr.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gplupiyqu.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gyxhftzov.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/ghsipkajw.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gdxtyevtl.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gyalibtmm.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gewsznbqi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/grmgjuqki.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gzkoznbdy.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gudbbvsfv.sHtML


<!-- 参考信息 -->