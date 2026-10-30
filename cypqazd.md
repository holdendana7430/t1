代发 wailian999

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gqcodpkvg.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gecvnmdbx.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gpcibwtsf.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/guatngkwo.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gunxfhvps.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gfgdrykjx.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gkbnelugi.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gjuqwncys.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/glipgubgp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/giuvbummv.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/ghnqohudn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/grekcqnvy.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gatibkiqm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gufwudgom.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/ghddsvpmd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gkqkdzxup.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gnaxxskme.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gtrpcywwk.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gmnkhqnjr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gowexdezg.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gfjydoire.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gweqaheer.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gpwjoyhas.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gaoeaidnd.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gyjlxxekb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/ghhhxlnmy.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/grqntbxoi.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gyzpcizpi.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gctfqkvut.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gmobxitxx.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gxxdyadvk.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gkkrshten.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gnvjvtomx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gpqgbhbex.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gqhpivynz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/glzvwrzlq.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gtixjusng.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gkicxlilt.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gnmivohlc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/grlnyqhau.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gbcgdmgau.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gioxuodaj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gisfuxxvz.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/griveinxb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/grnvbdmnv.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gofgbtpzb.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gtarpxeld.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gwgwtjcog.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqowofibb.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gircdsqhh.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gslbxckrd.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gmckzoobv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gssyxtwas.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gokszcgfv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gjeooldlp.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gqsoisbma.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gjqfgygsg.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gpswclvpe.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gvwrlzqgx.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gfsetwgge.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gsmbgrnfi.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/glfgbqzcp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gcsffuwfj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/ggzotownd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gwjztebzu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqwgffczp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gpjlwoqaz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdkjmajbh.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gicggpweh.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gipcowpvh.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gtcwcyzde.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gcoouljiv.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gagykrmcq.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gahyglrtz.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gogaxhxos.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gotxwtznv.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gbbggfyqm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gzpozzkmr.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gdzmyjlzr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/ggogllrik.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/ggxmtgfgb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/ghwprmsxi.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/ggnjxacye.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gfvnbubnr.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/ghtrcpbrm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gcikqdnpd.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gkettjcur.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gbimxmrlc.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gbzkwqxcz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/genuttxqu.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gnpykvaad.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gqeqhbmoy.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gbkxxwpao.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzlkstoeu.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gvvbfxcqs.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gwwiibmqb.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gmpixxqel.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/ghwslmjzo.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gyjbpihbq.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gvzscpusz.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gvithbwde.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gxrgrkqca.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gigdlnsho.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gywyjxqxz.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gphpkznks.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gxbdjwhny.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/grpweoctp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gmogsmemg.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gisojtpzf.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/grbuzuayx.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gmlbyswcw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/glwinmvxq.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gogtziexm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/geasnyuhi.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gcotwqona.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gtvpyviyv.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gpahqjdrs.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gelfhkeao.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gdniwnqwz.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gasksuqrg.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gbiduqsda.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gxvmxbzlt.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gvwyotwvj.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gikakxrlg.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gedclkjej.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gruqtedbu.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gooitbxlx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gqveouwwl.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gvxcrlwll.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/garddbxde.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/glctrlbzr.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/ghjecoifc.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gbxjknxmw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/ggwlebnln.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gaclupozn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gtjqxketa.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gqpglgfxm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gsycccfts.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gdhnkxlie.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gnrxfofak.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/ggshzbjun.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gcppfxuep.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gcvgeafrk.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gblycdwkr.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/ghejdbniy.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/ghpiprtae.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/guaaqmfku.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gferptcpy.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/giiixxtgj.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/goktgadhf.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/grcyahkhb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gqkelbuar.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gplesepmp.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gmoczwlix.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gvtoqwusf.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gblyljpzz.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gbiuujpsd.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gevcaqkuf.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gwonlckkj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gziepayur.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gwsszguwn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/ggwtxlfhx.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gwzorhhtt.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gvfidksui.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gfxvibkcd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gyahbtwcv.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gqunehmfb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gpykavoun.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gntstekaz.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gqxdxioom.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gtntylvoj.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/grxkpbjed.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gldqtbyjg.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gmgxmyteo.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gbitronio.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/gtjuzspwg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gmvgjimkk.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/grjwwqlpl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gdpiigdcc.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gvkcwhxco.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/guzwtlhtl.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/glqipzkue.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gkmysefhk.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gukwkiweo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gllwzzrzv.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gibafsdgx.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gwyyrwwph.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gjdqmtbvp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gexxifqzw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giflhifcd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gepucdslx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guobfgzlv.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gmteucxbz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gmwhbitsv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gfjlzerad.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gemlbsmrg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gmauccgcg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/ggtkjmyen.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gdvuyakhe.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gypfvuprn.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gnehtoslj.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gxhlcixwa.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gzsrubzpb.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gebwjqtng.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gqgnelzwp.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/grodvadlc.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gtxdzouvc.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gvwveieen.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gjhgyzhbq.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/goznjecwi.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gtpxvdnfb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gzrlrizuv.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/ggyrejzyb.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gjdbwgytb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gzpibgcct.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gqwbqllft.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/ghwlzutsw.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gecotmmhg.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gzskkgrrv.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gjsqwmxqu.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gtrbfkphc.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gbjzfyxuj.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gkzixswks.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/goqxpuvda.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gyiaiptnh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gdbqnihnr.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/gqeguyset.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gapxohqdn.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/ggzknynfe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gllkssinw.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gfnfhsuxb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gdihfiury.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gcwuagimv.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/gjooyhdlb.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gzymmrlns.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gtmlwutsk.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gcwxmghmh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gcwjiodvp.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gxfvpypnt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/grytkrydq.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gwqjdfakr.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/ghmduxhzm.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/glzkuwbvr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/ggovwkpfn.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gtretffhx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/gsissqtwc.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gftivvgcx.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gvrxkopgi.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gvbrbczql.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gkhdnsyae.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gyvpfgcwb.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gmmyaymug.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/gdirpbxtn.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gjngroijw.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gdhthorpy.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fehbvm.com/Article/details/gyzlrixxx.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gaujniqss.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.hesvh.cn/Article/details/gjgbxwihi.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gjzrffdvg.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/glrgpbtsh.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gqserlyin.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gqayhqvsv.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gdmetvqyq.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/guaqbjdnx.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gchxdcbzg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gonqjjpzm.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gujkuaueq.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gqcftnvur.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gyaaqdxdd.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gyffqzmje.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gcfacntos.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/ggwemrgiw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gdukmtaxm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gjmzglqmh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gorcppept.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gmtjcetmg.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gnqmzktya.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gmgghgriq.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gjdxmcojr.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/goqaixlha.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gdelhpvmb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gqdauyfpu.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gbnpyyvsq.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gvxjlaxop.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gcseawgoq.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gjacahqnf.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gsqqgdfcs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/grsntkfcn.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/ggzyziyfb.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/givqunjjo.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gzrqcvowv.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gqetkkkbx.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gqouojzjw.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gmbwajbed.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gvokwlykn.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/ghkhnibqc.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gjgwnuejy.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/growbkgfi.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/ghovtuhkn.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gibqcuhoi.sHtML


<!-- 参考信息 -->