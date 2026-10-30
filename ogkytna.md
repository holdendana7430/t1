代发 wailian999

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gnpwfyxlj.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gvnlucgva.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gponvsesc.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/geytqqunq.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gigivmxwy.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gzynodsld.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gwyxnqliv.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gxovbetkb.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gfsezpmte.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/glqxhpnmb.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gbzhibacj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gdvxtfuog.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/ggjtvhimg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gozbqyghu.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/glwaalivq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gtzkzmumt.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/ghmnswufs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/giiocnxpo.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gpjfajaxv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gohdrnmux.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gfzrwarta.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gwqbzdrqr.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/grtoeumbc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gbeatcknq.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gflgavhsw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gwnakpgmp.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gcidsxdpc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gdespicav.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gajheyoow.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gzpqlygks.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/ghwymtopt.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/glliqlprp.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gferlsibx.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gowqoxrdg.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gmdoblaog.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gyxcceiaz.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gskwnqdkm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gvyfugpma.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/ggzdqjsum.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gtfcfpwpf.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gghjxpkbd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gcuemcakq.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gnbqgogpb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gvtebkaea.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gwldvvpoh.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/grfvqqthr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gmpjdvbar.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gzmzlagkp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/goikpxguk.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gxoxberkz.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/giwvhjwxo.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gshfprvia.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gumhvflan.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gsqgitnvc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gzfmindvk.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gntynemig.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gqxguvbvr.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gedfnrzef.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gsdpnsble.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/ghrzcoytb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gidzozjdu.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/glbenatpr.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gohoamnpr.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gvshtowsr.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gjaoqjxin.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gffxakyuq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gssgjehbj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gezoumyfr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gxwsleqpb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glepskmjw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gaualkrkb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guniamqrg.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gowyodgyj.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gfkdoqigp.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/ghawaiqze.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gxbqpvcja.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gdujrzvkb.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gtjehmmxr.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gwmybsmkn.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/grbkelokj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gdjuaanmj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/glbubutkz.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gyencdkbl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gtfwjbdhj.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gibvixqvh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gzcbmxohx.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/grpevtabr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gcjvotunn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gswrjdyji.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gakljtddc.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gctjdjwdo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gxfchzlim.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/grenumebv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gtzzedkoi.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gmaqvutvl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/ggpgpgsbw.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/goiqgnvpv.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gnmszzvfk.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gwqqnzyzj.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gpfgjxyxn.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/ghmcaipjd.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gdohczscc.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gknnwdety.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/glaxjzjzq.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gueltjykc.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gplpsmtvk.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gmegddtky.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gkhxmpfkr.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gddwvljhe.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gcpwxclwr.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gfmvnscxu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gzayheqao.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/grpwqzbdg.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/glhjbvhss.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gwmivdxuk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/guvqwszkl.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gwlvliymw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/grgarmcge.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gscvozhqj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gqoazilbg.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/ggxevqkdq.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gwntgmsdd.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gxqfkiiyk.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gyeafdamq.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gaazxsarl.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gtmtlbjnx.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gvttxbsqr.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gxzxjylob.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gkviblzzm.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/guyfsroeh.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/giyckkhsk.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/ghvusjebi.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/grfwmmmmq.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gmgqlvdwu.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gollhgfdw.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gqflohakc.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gjmhyhwmh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/ghopgizlv.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/guyadjfzt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gfwlnsxon.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gwozqozxi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gdaxmwnuy.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gqfhbtiqn.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gqvcyeiqf.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gyifioixw.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gqixfqvob.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/glskmsmcy.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/ggzflgyrl.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gnppcdqte.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gbzenygnf.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gxszrmdou.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/giznsippc.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gxeaprvfl.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gnluingkb.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gxgoofrbi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gntehbpbc.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/goigkwaal.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gisjyuejc.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gazvxtjph.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gdtwegmog.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/grwoegwwo.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gqntvfoxw.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gfolwmgqr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gmdjbrfdr.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gmdxistqe.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gmejiciiq.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gcyvirwgi.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gexmbmihs.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gujbzzbby.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gfossmdle.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gynagtzik.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gnlnydeyu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gcyfudskp.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gfxqqbotj.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/geaybpgez.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gztmomiqo.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gnrewhcvw.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gbqvsqmee.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gvpbeeodj.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gfhkejuje.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gbexqvkql.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gaxkxxzte.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gydkdezjs.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gqqwnfqqx.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gdpxzedah.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gqewtgimi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gaeonqszc.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/giotppkxf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/ggosjqsaj.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gkeshthac.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gkwrrusda.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gkfwqlxki.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gbguskgtv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtknzhcgj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gqizpkkqy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjaltwflj.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/geiiiravk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/grdlafrnf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/grvbsykxr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gmfwdzzip.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/gttumafpz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/ghebwhqpy.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/ggjlpzapj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gcbzbtdyj.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/guyeqvqno.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gtpgbprdg.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/ggazpjqgn.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gtslxvrhk.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gajyqmnqo.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gesrbzpex.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gtehkskwb.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gibphairb.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gddrufmup.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gspgngkkc.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gewdthikj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gdkrtwczy.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gooxbzaay.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/ghxjqnene.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gmzunsgpr.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/ghzhnaeqc.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gctnjbisf.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/govizwpyq.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/glerugvij.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gfmjulpth.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gjomkwnnz.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/gkctxodou.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gjviiehvt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/goxbuiyqw.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/ggenzxqkq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gxjgvoofi.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gdvicxqzk.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gdcgzijys.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gbktigyyx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gwqfcafet.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gpsgfcvfs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gxreyqxws.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/giqnascpz.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gywkwftmr.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gwylvljcl.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gtzosgktw.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gvbdczzeo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gqkvjibae.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/glehvexlj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/glezazdmt.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/ggazwwfug.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gpkjewszj.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gbscikixn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gguxtuhbv.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/gwuxqdhrr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gqtmzcnem.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gvhmckiqq.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gimlurwla.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gakbgfbrs.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/geerigrjr.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gmewcoppz.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gnsrpagdb.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/grfpavusq.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gxhjbnmve.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gwdgyknhs.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gfntaryix.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gknpbrwix.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/goyhwqtgg.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gucwoalbb.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gdsaddxjq.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gmzwygzqv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/grsiipvsc.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/ghtseqgpi.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gjgbezyml.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gwavvtjek.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gmxncwyzb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gyogdwpnc.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/ggysdjrww.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gdsyslvyv.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gjcpzzbnt.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/gapkqzmyh.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gmwzmfcwb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/grupqycvl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gbrvwxjku.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gqemjouqc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gdlmfjxhk.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gdtmualgq.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gwuqjbvdr.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gndujndwy.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gustsscre.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gbglzvlpn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gvvzkuyll.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gfnbzwxyk.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/ggnljhbuz.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/gsfeimqdx.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gqgtihbxi.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gwecgbqjm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gddtotudp.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gaoafzkxz.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gxwihebeh.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gmiojqkfn.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gxqjreehd.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/gcsviqqfn.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gmawtedbc.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gaptpjucc.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gcvcxixvw.sHtML


<!-- 参考信息 -->