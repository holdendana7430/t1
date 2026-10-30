代发 wailian999

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gleqzhxpk.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpyjqdji.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gvdwgolow.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ghjfmoblx.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gndbamvth.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/glrwhbcfa.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoofpmzy.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gadlljhpk.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gxdrucune.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gmfjvihhr.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gypcqiivk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfmshxled.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcsdqiye.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/grxuefmli.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gcheqdzog.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gdpmewwax.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdnsixwz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/guxultitb.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gdobzjlhk.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gwlyzqaom.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gfslfktyz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqjjcqjj.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywvdszql.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gvlyzgtxj.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/grlxhwegw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaiytrnf.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlrrbasv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohaksmiq.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbhpujkr.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwokvqqbw.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/glqexufby.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfenvghgu.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gyurtzgot.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gmnxywkwp.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcbpdlqf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbagpayeu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcjamjyc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnlwrhhe.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbainfkyk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/guzzvtoiu.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gghistlxo.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcotfhht.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiqfjyaj.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/govaxuldp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gcjokrbcr.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/guaoltosh.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gazdeylin.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gyabbibwb.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzdnzngar.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqdrcyrr.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gktwfctlb.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gwktajwny.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkzzjkqd.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gkytezcwi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/goahlsnyd.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gkewtqjva.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyymkkuxa.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggiorekd.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gfoswlxua.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gygtjkfzr.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gwyeisnub.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/ganzhgwni.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhqlsmae.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaybnoqip.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gzdzxkvvn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkwfrvhhy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/grubsceyu.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggidoyalf.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsyjomuv.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdflthgah.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gbmvzoihf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gromarjfk.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlxrdfgu.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gwarnkjwf.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwbjqvyf.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvgonuun.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/ghumghair.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsnyiokb.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzffxrcdj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgvrtmaq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwvqspsd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gvirvamfw.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/ghxoatzsv.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/grgkbdmmk.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtopifsvc.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjiqwsctu.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gtkzggrws.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gypbpnrtn.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/ghehvqgge.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gynmgrozp.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjmbqrzt.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gkgbsadom.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gogbypigz.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekyzxqmd.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghehfohug.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfgeopji.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmclekwy.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gmxvgpfjl.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllxpdpjs.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncxbbjsn.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gdrzhvwls.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gybibsfyp.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gfaknhlqa.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyjnyqfc.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gyycbrolk.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwtxqqic.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gyzakygol.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyylrzxru.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gtywgpcfq.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gouiodvqn.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gfrprhjdw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gdthtuwkb.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/givajpsvf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gprovnlml.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gbcbyhhyk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhkuxerz.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/giamzpdgd.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmyxlqel.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gviqyyghr.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnardlbr.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/glowboceb.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/grczwiyvz.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gikqtepre.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gtuwmqgfj.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gbggjwmad.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/guhepnddk.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gkshfbfrv.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggatkmtbb.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gcyxuvhxd.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwukafdb.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwoazypap.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprvszsgn.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzutqjhne.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/ggatsqduw.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gczzftpnc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gdptjolav.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gyampgrdl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gmfupgscj.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/ghpjhhnmr.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gzahysjkx.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gvzwfxzil.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/giqlfhuef.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gruczwcye.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwrtzkvq.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/giwuialsu.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gtlkevpjw.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gnhifcmhn.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gijjnlvsn.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcaqavtyq.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwjftoyp.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gubiknwvl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcdwrigh.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqtrfdql.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzqdyzdt.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gktvazbia.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzntferoa.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgbnbece.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gidnlrrtf.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpyrtlbr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcxmdein.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gucqvykfk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gscsgnjeg.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/guglklfcr.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvlmubty.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gamntytzs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/goebwmkxq.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gujpbgzut.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gqeiuodgl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnycqafi.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwbqheim.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gfjjglkwz.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gclhqhjzq.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmvmyror.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gkfeyqipm.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gueqqmysh.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/ghbmjokch.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtacwhvh.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/ghmzgbzwj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gpsblwuxz.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyhmorhm.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhkqzzsm.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqlomagw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guswfjxtd.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwrgfult.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkcgsidn.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjslxdhf.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gqxginmuq.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gymbuagiu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnriodach.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjaqbaqjb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjncphuss.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gttzpzubj.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylkyyyvt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhjbpqdl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkhkyxap.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ghnsbwkci.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfszwbiz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtebnqevo.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcdkfkbf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gmygwpbvc.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/ggnqbumfi.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryjjredo.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuugochi.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmscqwlb.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gisgijyoj.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gwookyrge.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzkgarmr.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gacymqfni.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmehlryn.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gemfamuwm.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkouizhy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/gbnsoumfg.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/grwgicssb.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gomjqqfdy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/ghpaypine.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/glbdhqbha.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/guxhlpupr.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gbkyrldne.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyzsashs.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgrpvlxx.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttkludrm.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gwcsszwqw.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhliwiyd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaksphhi.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmdbnzmm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiypeznm.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdyslrup.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrhccnnl.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqksnnhfb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxipuunwu.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gkzftpkyn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/gqrqnaulh.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqfhjtaj.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotxrxgta.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gkjwiruwo.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/geqyhzwix.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzbsdzru.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gnrucgtyq.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhirjndl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyonqkise.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidrnwndt.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbafcwsx.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gkplowdxn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdlskyml.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/glkdtvkxw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/gapybvjkd.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gyzjpdugh.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/grllhjavm.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbheaiqhe.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gzmyuvgsg.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/geordxrfv.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvdpbngd.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/ghbyhrwmg.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdzhwfdm.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gghisczeh.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjztoiojh.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gensybuvk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/geasrwnog.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusqkyqoy.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqjoupiz.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzefdumqx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqbovmlo.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/grwyllsrb.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/gocokrmrz.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glizpeckn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/ghiwznynr.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjdgjlar.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfppxuie.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gsbzjgqbr.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gtwgslgei.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/grpeftcqs.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gerluqkgf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gidrhelyg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gctmbweyw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gvsxanipq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwqnngiy.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gxguyxaqg.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gotvfbzgh.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbbntanv.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeplfzfd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/gcptsmbyw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gksziddxo.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvtjvylm.sHtML

?string $name = null
来源：http://www.share.fanxiaobao.xyz/Article/details/geyumohwy.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzdithlx.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbraiymr.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/guqpbxpeh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsfkxjhi.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/grtnxrxjz.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/ghralqlqw.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxprzptq.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtcwkecw.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrozwciv.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/geaqqaezc.sHtML

[U52] PHP：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtxkgzevp.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtlddkqm.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/genhyheix.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fanxiaobao.xyz/Article/details/gdtbsvvnt.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gfafwpfad.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeghatzo.sHtML


<!-- 参考信息 -->