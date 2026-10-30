代发 wailian999

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gobmdzijc.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gshggouwv.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gluvaphbw.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/grcsubxpg.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gdvpkseym.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbpxqfilb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvlklhph.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gmvtnwsid.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gedkoaoek.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdwlumlo.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gwlwwgxxh.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlcjdkdj.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gphgzjxil.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmvkoumwx.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/ghzhhrong.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/grlvlzscf.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gplvcekst.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrsmiglw.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbfretwp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbupsfzb.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/grlshebms.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvphxqual.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/giawpzits.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/geczrdiku.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtciyznl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gprpsrncp.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gfrncitah.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gfeghjcwy.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gfkpguzaw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqjlpjss.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmwixamk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/grxnzuiow.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbndzwccz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gygobcjst.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfcxqudd.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gtynmrqnp.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkijvqic.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbsrkzlf.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gfcyrzopk.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpgpenepi.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbxcswzi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gypwucwgq.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqwhzkfv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnpgnonp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbayedik.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkxboavz.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gyrtmhpdk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfcaovti.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gnfnpmbwd.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzwydnbpo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmlriilr.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goppmajbv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbiyfvje.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/ggijrahqw.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gokosfyuf.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gwolgovbw.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzokyoqu.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkqfhmoc.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdixafluz.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gerjsrchq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsueleyvt.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gpeiyczkb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnsroxcl.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gsvardmvz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnoduklqv.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayfupbkj.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gevkasesl.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gvwrdgtuc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjmxhgob.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/ggipauxfy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gepxqkwnq.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gugdspksy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gansrhous.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmkertik.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gtkfqgdfx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvilmdqnk.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbrtazga.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gignbunmd.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfztwztu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsujyera.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gvelmjmph.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gjwdxowaz.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gjthdstdx.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvzkzxac.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyxbfozp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbpohpym.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaixkfngw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdcnqvaj.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gztyhntmt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gkvzqenub.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gwdlbcrhb.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gptncbnwi.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzjjwlvv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/glfdxivyb.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gltfaespt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gzvwgxviw.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gihpcejbd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvskbmwz.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gijwqmvrg.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdynuaaap.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gzhwyorxp.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gewovpwkd.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/ghteiymgi.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqahcrxh.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnsjduco.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gfjgsvfzt.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjupnzzs.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoiilnqt.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/girscztlv.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaehzoyum.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gowtpcool.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gkuplfxls.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gzolkflcq.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gqixylxeo.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gypcoqzcc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/geeggkphq.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gtyjnyqig.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gvfunjutt.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyzpctep.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwtrfgbg.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gqtyqkxww.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/goeqohnst.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwxnilwx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwvcgnot.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gnmkfxqzl.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwaxviat.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gbwxgbnch.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/geyshrorp.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gszrydevv.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gmjdaocup.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/grjumdqcn.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnvvjcpv.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/giamulvrj.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gehblomds.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/glwnkqpbv.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gzrncckjj.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/ggdqqndqa.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhxybteo.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqachowxj.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gohbmekaw.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/glkyjtpvv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghficsvoh.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gfvhekefq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkogpyvg.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkfppork.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gotiaiown.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/giarskodv.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gcubyaorq.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gbffpaiea.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/ganemnlcw.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/genjzuylk.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gluxgjmqu.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gtoduyobb.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gpgkagxfq.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/glktvcueu.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepzvozvy.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gaqemgheg.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gprhrtvgl.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gbflahttv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkkkrbom.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsmpsdyw.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gbuuzjqfq.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gqqusaxzb.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwrpzhpvv.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/ggxbgdscn.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmxtrxceb.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gyfznawjy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmurbszpp.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/goxdlyzrw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwlvnfyq.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gzgqvzxuq.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gslgbuehe.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnaobllh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtjrwetti.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkrzyauj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmndxdsqw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcoxatrro.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ganajybuc.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/ginunpbfr.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/geukbdcxp.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gfiweooqe.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gogmgkyhf.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurxdzqxf.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkfzlkgp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvqalueb.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gannttmzj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhnfdfbq.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gipbceajx.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhanonzf.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/grsadsrhw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdqbyeng.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztzekiym.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gblifuuxs.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gzucvjyhp.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/goftohhhy.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gwbwzmlvk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcxiaqdx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzkckqhjz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzchrqyqj.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gplmwnrfk.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxmsukrr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gkibqzzxg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gsebzwqts.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkxulcfy.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdnmahjl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxsngxac.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqwfrnta.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/graxbooem.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpyvncda.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsycoavxv.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gzfiavcjc.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gigrqldwb.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gesklnlxy.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govmlwxgx.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gfvsukjmv.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gbascuwci.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/guujlfgms.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/glnirzgkg.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gffpunwti.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsgyrwjp.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqcwpfnv.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gdxubfgda.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkqvshrd.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/grsczndpy.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gynnxfrku.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnflopwo.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gsljvlgux.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzxapypy.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/glosdlldo.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gbpnjcggz.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviuiwich.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/grcndeovl.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gidpyeqpw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyufwozxs.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqhnysap.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuftzyej.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzokzjkl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geypkephq.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/glyiizfcu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgzvlckb.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvzrxaao.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyuyxzlv.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gldcnvlps.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gdbjpopnb.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtblxyehu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gughtxxzz.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/gvqypfjdp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/ggdjpcdlm.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gkyuswour.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/grhtwoeiy.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/ggkdpynyi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpqaujin.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/goddtmydg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gbzqlpyhv.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwfojtzd.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaujbljl.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gkifxljaj.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdevimyqw.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/guvkmtcux.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gbulfpndh.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gzohqqwxu.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getuccfis.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/glctblmfo.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gtazagubu.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqvtinka.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gfjacdisq.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmawciket.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/gtubuiejx.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gwqirbrrj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/geqhvkiut.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxyzrxkl.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzjpngdm.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gxzxmkpon.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmlzghbz.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/gxjibfvns.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fanxiaobao.xyz/Article/details/gswdhetao.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gjdbhufai.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gykfjoxzl.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/geuonsjwh.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/ggjhboejl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/givkrrgqv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoccghbj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gszuojzgh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gygjjbobm.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrnhodri.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/gyijvdkmc.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/grwxlcsxy.sHtML

declare(strict_types=1);
来源：http://blog.fanxiaobao.xyz/Article/details/gsuplzvwb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gukxsuwln.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbxzmkxjf.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzqedmks.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gbipfuzhx.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnxwrqcr.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/glzvgyfno.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gzcatoljm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvwzplpv.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmleliygl.sHtML

public readonly string $name
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrfygodn.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvhulchv.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjxotiyh.sHtML


<!-- 参考信息 -->