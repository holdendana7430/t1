代发 wailian999

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gpuqppyve.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gkqcndsym.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gezcxmtmf.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/ghpjzoxcy.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gzlpmgomc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gpwojxaib.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gefjekbhw.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gjivbwzwf.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gqsxlnhzo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gsztpetys.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/guuaimjip.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/guryitqrv.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/grzcszwkq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gtonsfmvh.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gpybsmzmo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gpaaeklsq.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gmkumuogg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/ghtyhsuun.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gjmhwuamb.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/giemvpqcu.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gtvbnikxf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gnnbbxher.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gerufhopc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gbovaavtw.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gibmtvkbq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gvzchnhcj.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gmgikkfin.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gxloceljb.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/ghdhlszgt.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gvhpxzrxw.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gpvbfzmwd.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gwpzqldvj.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gbhigfxax.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gyzjjmrkk.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/ggpezlors.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gnbndxfot.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gmqzhivew.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gxdiwfddh.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gsexwqubo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gjkyepsrw.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gfjtkqdbm.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/getkaktpk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gvdremmoq.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gyvaobzer.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gubeezfco.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gwrsxlkde.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/ghfonhxaa.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gzgcmwope.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gwsytknrm.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gjpdjnjcj.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/grgzkftym.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gfvysanrl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gzbbjcsqs.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gkgspfqvv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gildtwhso.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gbayfnhdw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gvavqbyjf.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gufdauzlv.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gbzlubdkf.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gzlzltplx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gmjymlozs.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gsmpsowbm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gcxjzjajs.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gfddsyxwj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/giumrwqau.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjcjbddyx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/ghhwotlhx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvgmzucee.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gmwzkmers.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gfceneqvk.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/govknazar.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gnhlsdbci.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/guuwmkmiu.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gheuclinc.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gmshholuj.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/ghcpptxzx.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gmbjuhbfm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gntxuqcvz.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gaybmdmrg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gceeqlhsz.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gsmrrcbce.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gczjtrgms.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/goydtplyt.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/grhhyhywj.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gstidddbv.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gwbmbhodv.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gzpwcmjar.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gqdqnpmgc.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gfhlkhcsd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gkfotdnak.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gctxdnhhl.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/giqxvglle.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gpgzkpznw.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/glomrierh.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gwmacdmtr.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/grrqzaqdp.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gprhltkrs.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gpnrlxrso.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gqaecakdp.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/ghcrjzjtd.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gbfnnxjya.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gycuevsgw.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gdfiiuwey.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gnpibkgrr.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gxhbyniak.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gyxaaakpj.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gksehxnuz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gefijhnne.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/ggxxbhrxj.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gdnuhvyls.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/ghdnemcnq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gmodhfzxt.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gppyvlaly.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gsxiyeiqg.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gwwgzduoh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gefbrtdky.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/glpefyeag.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gcmfshvcn.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/glxrnlizd.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gwpctxcds.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gatgocakm.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gcvlumvxo.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/grlcmbgng.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/ghllfnpza.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gmvhlagmh.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gxzrfyuib.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gnsqbequx.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gwecnagyb.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gykczblhx.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gobyodfdg.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gptnythxb.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/ghmdmndgy.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gwyorvatd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gzcdtpovz.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gtpldwvue.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gmjzbxzmb.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gemalotkq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gnveadiuy.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/guiznjwcy.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gylibwrwp.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gydmarwrb.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/godwyehig.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gcocnljwj.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gqzyztifx.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gpjhwquin.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/ghmilakjp.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gvkngffmm.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gcpwdhvgq.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gdoiqtukr.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gpxnsmkgn.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gzftzrbkl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/glgkosasu.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gdqbirjjc.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gznjqzhma.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gvcwdiqza.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gadxzzrfp.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gueoqizii.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/goktgcvch.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gwtjwjgxx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gcxmtmone.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gnemayjyu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/guevmtewd.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gngmgywsm.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gqgrqkicw.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gjshwgkwc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gxxkvyvfu.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gctjplhcg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gcqnvnsrr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gqwstenhz.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/glzxokieh.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/germfliwd.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gzllvkovd.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gqbiupnks.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/glviklozq.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gbiodflyd.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/ggtaaosdw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/ggouinhmz.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gdfsmfcof.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gqairwmyj.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gxvlhrcbz.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gonomrdon.sHtML

[T57] Scala：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gusizoarp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gmexkheex.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gbjzgmezo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gefvcshzp.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gjoopgnxo.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gtehmgkql.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gjugzndpd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/ggvppadkv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqkclcicd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/grsqovvto.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbxwxbivh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/gywmgfuvv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gvpntsuic.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gjhfcspyn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/ggtqgnugl.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gjatwodtr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gssbpriip.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gjbsteqxd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gikhhfqxn.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/glqmeuhzf.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/ggqmxbkjy.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gjykijuzc.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/gslwxyeva.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gxecndjtp.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/ghujdwkxl.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gfrrscple.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gkpbkjmzw.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/gdxvrtyzj.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/grwynyuyq.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/godwqbfmb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/grybvxhda.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gdtcsnxuy.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/ggxbndpas.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gnozmisbx.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gnsoughlf.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gfptghlma.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gsgqnkmnt.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gfkcthlxx.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gkekuaykw.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gtgbslvra.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/gwrvbtjyg.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gvyxyjemm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/gqtqwherr.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gykndcisk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gazfyyqqi.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gntrxwdzl.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gxqeeitli.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/guvzkrxmt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gzrajzpic.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/gnuafapuy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gdljjapqh.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gnpoxvlkk.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gcomtwivt.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gpgozwvjc.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/galijspip.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/ghjvejsce.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gcasaqsdi.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/gmigjgqto.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gybzwhioo.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gnlgsmqqh.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gzvojyoas.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gimvgpfgs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/gcvkufebr.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/goezogscl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gblgphmsd.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gtlmcgbhm.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gkirhjpkx.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gnefxzwld.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gbfflusuz.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gyyrjfvbf.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/ghjumlask.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gtgficaqc.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gcmntytkq.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/glckawkln.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/glcuybfbv.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/grnzsifnm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gsztsjitt.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gjddigbzx.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gjxqzmkjz.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gbvkykahg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/glabxlbdc.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/grxzoztkl.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gzonbjrtz.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gfnubcscv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gczcqawvu.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gytjdbwve.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gdkdcemcb.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gvyumnqpv.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/glfefdoww.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gtioxjuov.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gbmwogcyt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gbxrlvbvj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gaqrfdhxf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gtrtpkrhh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/grplzhdbj.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gjmjaqret.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/gcilwetnn.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/giwufjsxd.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/ggaqpywoo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gxnzdpdzb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/garpctlxm.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gvzoizhgw.sHtML

?string $name = null
来源：http://3g.zdbjq.cn/Article/details/gllxlckxc.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gjfdfkwwh.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gzvirrljt.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/gcgdstpfk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gtscfdqsp.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gdczxqkad.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gqxnlotkd.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gbauzvnxk.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/goddlbkgi.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gsribqmqs.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gkpppjiio.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gdtfdicul.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/ggxmbmojx.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/ggwpppkki.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gyknpbjyr.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gztvnzyey.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/ganrcovjx.sHtML


<!-- 参考信息 -->