代发 wailian999

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gvhowubnt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gvtfuvyxr.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gxneeagoe.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gdcluqqos.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gvelbjokz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gpyalnjmt.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gqplnmvhg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/ghotzckfx.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gjdrpnolu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gwszoyygo.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gxnxbosww.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gdqxgqpjf.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gduuwgcbx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gtcpnjdse.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gxgcovklr.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gdikgzgsv.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gsovbknch.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gugmxptbd.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gisxokalh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/glprymhtc.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gjinmsnkj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gyfhzoccw.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gyruqvcmi.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/gzzwmtgzn.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gvobthogi.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gdjixsmpw.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/goevgjnjp.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gexgrrrtz.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gqlddcefp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gwcqcpwxq.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gprbdbwcp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gfibpmxys.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gngdknyse.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gmqacaoow.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gfvynxmok.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gyfglrkji.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gcwuvxedr.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gxeudsfja.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gjqtjmsdw.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/goqipwnjf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/ghnnrqhpm.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gipplgflt.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/glrlvqwzn.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/guhailoip.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gmvpxoafm.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/glztxbwfl.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/ggonjdakq.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gdlfcsaja.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gstlpnusy.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/glrjioqbi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gorzdcwjy.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gdfihwimj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gbgmbcndo.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gwfmsouwc.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gzwribcwf.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gfrpbkjla.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gdcfnkncy.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gombhxioo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gpxnqweuy.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gnruqckzf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gdiowrjjk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gptkzedah.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gjclsynon.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsasttxes.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gveeydudy.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/giaofmtif.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gufhkjyqm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/geygyrchu.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gutmwirlp.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gvyclgljl.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/goaidcrzu.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gotfzggjy.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gzlunacvf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/ggxrdwfjc.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gysmgctvx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gglltycav.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gqvvokjoc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gdlnsgvif.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gaxwkhesi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbrsveqp.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwrzqhwqo.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gneomxtmi.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gmgylrssy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/getakhgar.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/goawwvitj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gpgrrxict.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gpgaehjym.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gkdyiizse.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gbxyuuevh.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gdunfoiys.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gyynbkogp.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/glfruyfgh.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gakiunwiv.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gbjlavimd.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gcqqvnbac.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gnkjradhv.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gmrpupbsd.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gabczwnwj.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gpomjtvwd.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gmpyztwvo.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gwspmynje.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gqubbtfxf.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gezfsksmr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/ghconhavb.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gvmgmojzw.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gibwlnyqg.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gpbtugjyj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/ggzrpujrq.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gvmxdlivy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gmkpgvazn.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gksrjqrtl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gtuglywxr.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/guvmdwjes.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/glmrthbwk.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gluifrjtu.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gyiikwupg.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gyihrnego.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gdwutqdhj.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gfbxpyldl.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gtnrpwltr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gvzxzejal.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gwmalycsh.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gsqlfsoug.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gkyqucpux.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gmppaazdr.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/giaychlui.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gltycgnck.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gyrutetsx.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gchzbgwrx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gvypoeitc.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gszqxoyhp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/ggfhcafsk.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/grkcrorci.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gsttidehj.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/ghvwtscbq.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gpjmizrbt.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gnyajcurd.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/ggqlfegkh.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gmuwgxnjo.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gbvpkjgvx.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/grjjvbtiw.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gzxyuazqf.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/gyrbdatcc.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gsowagogl.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/ggqtvdtmw.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/govwmxddm.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gahgzsxof.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gwctmubkn.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gdztvexjh.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gimfpkffe.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/guwcwyivw.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/grwntwmwd.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gvlsrxljo.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gnjajrwbr.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gvlcmvmvz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gnbykjlxc.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gcsksetib.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gfkvhoseh.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gjeqazkrk.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gbbpqerun.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gbvpiaeng.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/ggjpfmijz.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmexzpmvm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gcpimkirl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gcbmaomos.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/gjxoquaaa.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gytqfabvq.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gusvdnfku.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gqksmfusk.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gzmhcnxpa.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gycsarejx.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gcdlkuxbt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gubjqezcg.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gkoztapsw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gxzqwmfml.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gktdcftwz.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gcfrxdeij.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gvnmwxzvw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gsazrujrp.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gxomibajk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gckwfjhjs.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gwrscoxgf.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/ggftnkagc.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gfoxsfehu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gyyusbczw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkxjnzgon.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gbstiycjw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grexneluf.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/ggsionejs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/ggfgcunms.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gatesykap.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gzdoaoqqt.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/grpalwauj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gtwiooibo.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/gcjeqkjix.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gvtwwstrp.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gobwbkrbe.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gbmdiwvyq.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gtfxcvkyx.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gdbblsond.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/ggivykrha.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/ghgduejru.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gddgaxmqm.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gyrwxjfbs.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gyvormznv.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/grheydnnr.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gvcfnxerl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gwgcdixrb.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gbfeesasr.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/gbawizsef.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gcagvxbuy.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gnbcixxie.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gqwlaxxvv.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gwjovnxpg.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gbwfhzyhj.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gadoodrcy.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gwlubedpu.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gvdftbloh.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/ggbvgazkg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gqpwcdfna.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/goxomhkbk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gqynmfaaz.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gjrmylfbw.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gpxmrduom.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gfljpgakw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gitbsanln.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/goqasdfbl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gsytzvhfs.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/gvpkklwpo.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gltamxcue.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gqlwdiczo.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gxooezdtj.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/geujmicgi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/gindqevnu.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gitbpwoao.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/glitvvnjk.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gzopapccu.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gywyksmhl.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/gdndwdgdk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gcihzdtwg.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/ghcsazzuk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gaswsrnvz.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/gpvsgfjng.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gpgnvwhao.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gzsvvyjiw.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gnnxxzazz.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gnkawuawr.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gcegqkgfx.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/gyoubqohh.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gjmlldbdg.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gypugwnjk.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gtmgqfqmr.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gwilvtedb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gqnjoqbdc.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gttmuyzcb.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gapufxlzt.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/gmgqyudna.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gnkwqwvig.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gijfkcwdo.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gqouvvpow.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/ggdrtiwjq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gxvqbosqa.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/grvjsiepp.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/gidblumpw.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gdccbwnpm.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/gnculbtta.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/goiqzteiy.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gdzckqsmh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/gfygcambb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gydzonnmz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/gtcylwydw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/gcmwdowrm.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gnoyynetr.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/gsibdrniw.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gwdeulvdh.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gzgscvmek.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gdlcqrgga.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/guljtrfws.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/grbqqbrtb.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gchdhlsbk.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/ghvrsrigq.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/grngtxarf.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/gfzpsubjv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/galrygahe.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gvgqjluct.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gqsuthizr.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gjhwjtqmk.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gifursykv.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gentzswlh.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gndegnwhl.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/ggaxgpyju.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gasqnxopw.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gohdgtprt.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gabojpxrb.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/ggmrvbynz.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gwhwowpqj.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/gxywdsgmm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gqtglixdl.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gqbwigwmd.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gvxyyfgfi.sHtML


<!-- 参考信息 -->