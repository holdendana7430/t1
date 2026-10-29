代发 wailian999

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gctfokwrh.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gnfrjsmns.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gxnkebufh.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gnvubdqzq.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gllsblmyt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gkarwhyre.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gfuurfqdq.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gvokwsosj.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gmncsatzm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gmzywrhtz.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gllhhmqee.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gebkwjrsm.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gmywfdnnr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gmhxbfmpn.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gxxvmnzgm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gvxejbchg.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gyiwygzgt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/glapvnivn.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gdpdpdhns.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gbbppknbh.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gmfxtbsxs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/grlzsnjbk.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gzmrkgyfy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ghbsjxurm.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gymujwpdv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/grxwwster.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/galorrjcd.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/givckfqjw.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/glznhtkeh.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gzqpqhuuy.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gahlspbhc.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gfcxvjijw.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gooakaxcd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/grdqqkreg.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gnyczfpbs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gtxaaxcat.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gdpuvwiir.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gkgebypsq.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gnvrbwnmg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gfpzzqgly.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gzyjlorri.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gucakjnot.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gerbviiul.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gbzkbzjgv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/goccbltzs.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gclpmjpck.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gyirpneuj.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/ghusyxogm.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gjtjnajcy.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gzzxufiux.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/grrhlreln.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gawlztyui.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gtjgubjqq.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gkcnivqqz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gxmjbldgu.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/grtmpbcqf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gksjvtvis.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gwtuckrxy.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gudlyqpqn.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/geyqlrwhe.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gmtbhdmsk.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gxckzycru.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gqeaqpzbf.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gzpjyfknt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gnodzdcte.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghnlsesez.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gtfawdkyz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grxnzfyzj.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gahmvgdfu.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gtsoevtkg.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gqdwuxhkc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gmlxlgjqm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gycmgawct.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gaftbqtef.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gpfgvfavk.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gvrxzluov.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gcddisoic.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/goiyuiuea.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gqhopwgeo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gefsquefv.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gfztavguh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqxzzdlhn.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gfxynqplm.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/guimjsmzd.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gozkoiaed.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gmbocurkk.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gzoonsnyx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gkouzxmyj.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gemnlugfj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gqjhiinie.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/giekazjpx.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gazlgjgjq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gufyuvlja.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/germxuqoq.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/glhwjcrjg.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gywdpnmsz.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gnlgniznr.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gkwdxptdp.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gbnuncykd.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gnlttwbvd.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gxvbstbof.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gxhteutqx.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gybhhrgru.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gpdakpwjz.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gakonovkn.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gxldtfybn.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gltvqqlvq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/goigfqnwz.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gfiqmziub.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gvygfhpvp.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/glgfaqqen.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gaesvxgdr.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/geqkfeqiq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gysbgwfqn.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gbkynzcck.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gohsqjiip.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gsxfbdsta.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/gjhcxyapy.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gszwvjczz.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gofpzgtab.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gsxguppfe.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gsqgnvzgg.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gzfxrhiij.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gsmkqkmix.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gmaaypjrg.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/ghjtzhtww.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gmbrszoww.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gkatyclhg.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gycjcbmmv.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/ghvsccifn.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gpbnfpgsr.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gtbaujzxe.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gabicpano.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gonoomzbi.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/guuzdgltj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/geuzcvgrf.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gnkpwbxes.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gsmdagtde.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gdxxazjmm.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gouqfzsjx.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gmzmkteqb.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gsqubjove.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gwxmjwmzd.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gwkfckplp.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gcgpypwxa.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gxpystlwf.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gvkdtmpjc.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gtyakkjid.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gmraxomfb.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gqdjdzeze.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/gluqeitpy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/glagyeuxw.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/guefwfdda.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gstwfgbdj.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gmeibndtk.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbfytrypb.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gnzhntssf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/guwryoxje.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gjqlqiwso.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gworxjqyk.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gappkmkrj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/ggutvqqnq.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gsirvnztl.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gcdyzutzt.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gyofnzskm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/geccdaxpn.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/grqhftgkz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gnbtljlco.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gngtdfsse.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gtkraklrx.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gzgrnaiwr.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gdkfjdwae.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/giempgrdw.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gtibavftx.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gicfpvujo.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/goruxkdhv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gqhugjcka.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gbngnjxbq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/ghbrzofuu.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gwtoamgnp.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/ggesjsoor.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/glmotnosq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gkdhvipsm.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gplqhtiyg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gndwndnzw.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gftlnvsmi.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gchzoldxd.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gpnhosbbe.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gzbmktnzi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvqandnvr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gazbdkxho.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdcoxzaqr.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gpcehsinj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/griiwkuhk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/grjogwjpk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gyvbfbnrr.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gcuogzdtv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/giobyysaq.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gnaosgbjs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gprmcrqfs.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gsloaopjp.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gvppvllvc.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gpvkrxjsw.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gbvvhdtsg.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/ggjuvsysv.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gomvlccxv.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/grqrgtwky.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gwcnrnuft.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gtpkhrbom.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gmgbtvler.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/grhnypngy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gqratsnpp.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gwjpdbmlw.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gftdspgdf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/glzafnwdc.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gzmbsicqw.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gefoiyoxl.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gsmpfllmu.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/geyvmzrgg.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gzsgwhxve.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gkxcxdwkp.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gfyemtips.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gkaejbssx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gllwdupnj.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gwqaollmo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gfhxfqwrj.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/gfxfsbuoc.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gygbwsejk.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/guavhpvcg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gddbfbjnn.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gvresuojc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/ghltzqumk.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gjcgffphg.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gbnbipyxs.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gucwerfqo.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/gfiaueyoo.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gsfrkiwic.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gbywgrwsj.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gjkwcpuvc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/ggmzdjekb.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gutkzhhyw.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/ghjhhixtr.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/goackbsyq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gsltmdkdi.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gdbgqsgqm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gnuaprwng.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gwwrusiwt.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gkksiehlp.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gkhhvilaa.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gsznzglze.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gbstxzlwh.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gwjtnenoa.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/gwkessuvh.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gbupkpula.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gpootcdpr.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gicvhfpxb.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gjtupjred.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gelcgamml.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/guucjevff.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gqamfyypf.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/glvyujyou.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/gthxkxxar.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gycnxqbim.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gslkgtphf.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gmasrngfn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gxbwivljk.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/giooucule.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/glkjejnii.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/guauseeds.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/gskjdnvpt.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gwehbwwex.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gvnoaspgo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gflhhgwlm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gmllgfjqb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gtawezdxl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/gbztrrfiu.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gwyvbibwm.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/ghoypqvpy.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gxmeuided.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/getjglmlz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gvkabhxrp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjzptdpwk.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gbnmbzhki.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/ggxllkpky.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gkbisypqi.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gpkwdigch.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gzzjzwhti.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/guqpfbpqz.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gcyngvmno.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gedexgbvi.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gywqscwgc.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gcqcfyxbq.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/gkquibywt.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/ghsmxgled.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gdqrtuoxz.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/ggerfjadx.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/ghlvyzcxv.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/ghrcxdvza.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/gpssbpghd.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gsumiavrn.sHtML


<!-- 参考信息 -->