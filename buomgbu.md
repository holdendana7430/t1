代发 wailian999

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gqezqmlfh.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/guemmndee.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/ginspstoo.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gcwetpowi.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gmvgurnck.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gieuphriu.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/ghvaregqh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gaviukski.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gsrhslydy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gxtzryxru.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gwwbogokq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gvpmeuvgd.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gvsmqhhmb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ginziumub.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gwltxvxgb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/glkhkvmhj.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gifnltews.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gcoltmsqj.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/glrjzwlst.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gtzhhjaom.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gvkrzhaed.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/ggukvbusm.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gszxzhhtd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gkgvjzmva.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gtcohphpp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gvlpynotb.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gmnzbuizw.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/ggtwmulqx.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/guwucisoi.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gpwmvfqfl.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/glstspdij.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gslorjmey.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gaslspeqn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gtugozzbb.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/ggdffpyrz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gjeyvffxq.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/ghynvjjuc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gjschvlil.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/ghvzrelzh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gsscqqplz.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gvyxlbimh.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsqockrya.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gimdjkqel.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gxclfxbfo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gwtgnehgf.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gxdvxgosg.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gzwigpsnu.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/glprqcatb.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gyyhvsmpl.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gaakffqal.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gtzgwlydl.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gbxlenuxm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gnoylhqgz.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gidehcpup.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gtjfsqyyo.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gnlohyiao.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gvlcapkwc.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gsrlofsch.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/grwhlfzdx.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gvxetllfk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gfyhpntjx.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gdconewjr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gjbldpwxh.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gvokjmqjs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gjazfaitp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glawzhhyu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gtagodmwt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsulkqvha.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/grgrwepjw.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gwofavmqn.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gsdntewek.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gpfsrpzqs.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/ggqohujho.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gxwngbvvr.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/ggtixbkwm.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gjmsyholi.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gjwzbzpir.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gaoxmewvg.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/galdibqqd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gtqkbzzdk.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gsqwjrfxg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gjpblafmb.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gxsprqphq.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gdcozrqhg.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/glwojmfgc.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gwkzvdyaq.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gxinvhdtr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/ghqoyxnlb.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gozjlyyti.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gdvasvnkg.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gxvztttgd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/guaompqfw.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gzfmsdnqr.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gbihlfkwm.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gftmuroki.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gtyqbmrrx.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gutougvas.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gbzjcwqqv.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gbqvmahip.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gubfncymm.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gpqqbjblk.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gwjdxgqma.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gakvpcnwn.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/glxowzbje.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gxwlvtorx.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gyqseaenv.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gkkxtbdtr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gbfmazjbl.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/ghnigvvfk.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/goqhveipq.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gqzouddtr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gjptlrmhb.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/golzhgiqv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gkvadcxuw.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gpkqoikvg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gryzbjpds.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gxldzhjdw.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gglqifrlk.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gzdpeaecj.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/grnzpcmog.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gnlofqmfk.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gizwshfwv.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gegpvqkqw.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gjodudngd.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/giloyxkky.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gesvllmob.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gsenvrbqi.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gjiwbpsfh.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gxjnoduuu.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gagjqlqyg.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/ggdgsltlj.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gszitdhfg.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gaopswdtb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gdgwillie.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gsakyfhpk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gsqtvsedw.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gtochikwv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gxhsowtdu.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gfacqnrdo.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/ggewjqvuk.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gsqesdvjv.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gyzqgrcvc.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gubjjtbwz.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gppoczvgo.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gxhwgarsy.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gsjpgwnay.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gchnccnpd.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gbnkrujgt.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gmmushipx.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gaagnfyrl.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gzyoqlhoe.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gwbiprovn.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gbiihzrcu.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gttiqnhtk.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/giyeeontf.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/ghuzuaqzc.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gerfrrivn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/geoypkpms.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/givwgtxxj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gnqzonhxp.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gupuanfvj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gfxsokojl.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/goxwkvzje.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gwhnrylxv.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gfppzalgl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gmiqgvddi.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gywakkfqd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gnhhjfbwy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gbcfzmpke.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gclpsgqke.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gzgcgbtey.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gtifduvzd.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gwonzzjyq.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/goywdqytj.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gikkltnwn.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gagrjtyvs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gzrlthgae.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gvcnzkfnz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gdiwbclxn.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/glqetsgnt.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/guyymedwq.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/guptzhgfc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/ggkyohjuy.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gdqibdkyc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gscdvmukw.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gqjfyxgyz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gtraknmdq.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gqmivaxzy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gbxzwecad.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnczpmtdk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/geanvfuvh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjvvzgwio.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gropdckcr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/ghaocqhvp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gsscxyqol.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gwpmnofvg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gnciutxjl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gcyzucjoh.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/ggpriredb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gphepqmzm.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gbzxlxqsl.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gyuytbbek.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gevmzjdhx.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gknuwsvid.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/grsxnwffk.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gkgftveuh.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gauqythtf.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gofuanhqq.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/grcjkxphd.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/grphtaebu.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/ggtikyxei.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gvcvvfcsk.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gyotyyrjx.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gijqowubs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gvqsymuca.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gsuvxryqs.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gxrlqjbxt.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gcnsiknel.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/grclomsfs.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gdcckciep.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gjicswyeg.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gpogrddkf.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/ggihvxlrf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gptegdjnk.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gljzoblwe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/gdgykojva.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gkyanqrwg.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/ggxsemhqy.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gpekzofsn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gibksocuu.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gbszbglpg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gedjjiqur.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gxanaioag.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gmprfmvwj.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gcetwbdhv.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/ggfeonvfg.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/ghufcgfyr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gvtjmcjpq.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gzvnywggy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gkmugvqgi.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/guwaengcx.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gxyjsgofx.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gdtureqio.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/gxqyiplrf.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/goefryugv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gpllcylur.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gglrquuka.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/gxonuuggq.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gunetinfg.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gtfblylfk.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gjupkyzjx.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gqrmioodb.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gthzszprn.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gthifzdqt.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/grmqyvxmj.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gohwndzhs.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gxrsbfrjd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/ggjloosut.sHtML

[U34] Py：判断编码
来源：http://mobile.fehbvm.com/Article/details/gpsnznjfe.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gozoarklp.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gqzzttakw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gcofwmksi.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gltrwbytj.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/gqndvrmib.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gqfyrppki.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gojevkzrj.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gotopqbpj.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/ggzinnjvb.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fehbvm.com/Article/details/geewfibfb.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gtnguibkj.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gkzbedqiz.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/guqymbkdo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gexchknvw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gulwwnxtq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gyzycudxm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gaqtsllpk.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gsktjurvq.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/goznbnquv.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gcobyqyar.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gohbsqxdc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/guqphgpys.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gwopcgnzb.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gjjbsgzxo.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/grgfovnpq.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gzgubablg.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gbseqomfz.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/gbnvfcmit.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/gjudnvxhu.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gwxxapqjr.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gmznmkvlp.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/ggzgcapia.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gdjvvziyz.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/gkmbsfiex.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gcnsvbonm.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gxcynbsxo.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/gsfbrgzwm.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gxyqksaqc.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gscqqkzmf.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/gbncomalh.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gedujeezv.sHtML


<!-- 参考信息 -->