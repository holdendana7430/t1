代发 wailian999

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/grrkeggzw.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/glukjkljv.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gqqhkbfbl.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gpueeuqpp.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/grcudoulr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gqydqfkry.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gafudmlib.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gianxgfbp.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gztpvxiis.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gizvshpfd.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/ghrmlyejy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gpojbnghd.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gzodrwpyq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/glqugkyam.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gkyugdzlo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gjfxwsasw.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gtfzmowel.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/guppkhmro.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gndnwglzr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/geogblpzx.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gbrgwyyez.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gvnhehqqr.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gfeczltcd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gveiegwuy.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gflkpuhsw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/ghvjwxyse.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gvmhhpkdd.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gwdgmzsfw.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gxczlzlid.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gnyamrivy.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gqtgqjfpq.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gxqsmomnv.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gjpzugdzd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gowhwsrun.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gkgzztgvt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gmxngriuy.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gzklnemtu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gbojkeksl.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gnwzwaoah.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gwqclqcnf.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/glfyczyyk.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gpnxfgsfp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gtttqdjrj.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gesrzyrui.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gphnfqjpm.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gmwpkyaxk.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/ggssrskbd.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gcphderye.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gdgcbwoby.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gdrzszsui.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gpqtfmiol.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/glwwyyfhg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gvyfvpcrv.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gfouduhse.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gxssczueq.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gmdxwbtez.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/guxcbdrar.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gssvvkfxx.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/giyksariz.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gyjecuobj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/glzubmsch.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gtqcvveqp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gamzhrpbt.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gxaeikxre.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gjnuocmdq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvasaaemf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/ghhveyhfb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzyacweip.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gdxzrjmdq.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gbqevotgu.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/glowgbqyw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gdbbouuzr.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gooigrhhz.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gjmjzofsq.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gnyeouqqh.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/ggvclcrnm.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gipotflgw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gmsdwtfku.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gsipsrhqb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gmvcvhdbm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gpolzfmcl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/guuhdbzle.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/grypmzxjk.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gvosvocpf.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/guaihmhtl.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gixeibucs.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gblozjecb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gnvmqrkft.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gqzbaouit.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gjyrpoirg.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/ghcmuexwy.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gdzhktptk.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gbekhabgd.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gictewcyp.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gzzswcsyl.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gevhcakzk.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gruhslwwm.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gvfiddwnx.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gmxeezphs.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gpiuvnxhe.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gfifrrucf.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gnrywsepd.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gfiasclgj.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gvmaayyne.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gifvnajck.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/glwmdcjla.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gkhpqelia.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gcvqpcfyc.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gwsrpwspv.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gwwitvjnr.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gsfutdwdk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gcwdaswuc.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gjwlmvqcs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gjwupnlqf.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gzvnbmhpf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gxvwsjnhz.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gettjeolo.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gcupuqqtu.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gqoiaiogz.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gyeszrmmw.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gclwruijj.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gpiqtdqqj.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gjykdbzkv.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/gspwojjxf.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/ghzqqvzgm.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gjpsqbveb.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gruhhrigy.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gmyropque.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gwbgdyakp.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/glfwikkhd.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gjkxjmsvf.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gbtxzztxc.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/goxwycxxr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gjpebsexa.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gzxtcozsk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gskvgiboi.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/ggqqbsmcj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gizgxeiah.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gyrlzzmwg.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gutdertzf.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gaiscdivw.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gemwwpqly.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gjqyrdovf.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/ggcrdbmoq.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gdyirznso.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gnriuvfxm.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gvltkxjlx.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/grxhfpnmz.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gogzmjslp.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/ginbfiasq.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/grerewciu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gedzeozqd.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gugezcrar.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gscexvbgg.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gjudbnjvh.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gsjckfhgr.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gbnotgpwx.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gykhsyfoq.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gmaqlcyzf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/grxaxhzne.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gjeauplkr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gnlohiike.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/glzxdvqtg.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/ghqgmvvif.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gzxwmylyx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/guqtkasbu.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gbdacgfft.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/gccrpdlhp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/ghnjptoqr.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gatdulcde.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/geugqtphv.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/guuhqwqki.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gaaafybpy.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gtnmvmdsm.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gpwclhiql.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/gydiorokh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gssjkcwhh.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/goevxzhrq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gztkcrhww.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gbtoadflw.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gttecngqn.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gaeqsuwhr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gyoxlapsn.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/giiunawqx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gatafybks.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gkiygakqk.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/guwtqdybj.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gmevcawhd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gdxykncrb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gndolgxij.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gaffqeula.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gltowvloc.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gmigwymbi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gaddbdroc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gddgbrkdz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gphmnaclx.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gnadftqah.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/ggaodrlvu.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/goaqzmnsg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gpejqpjsh.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gjkpftyhp.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gkpugvhux.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gnganujuj.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gmyfzaijk.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gonllgpiz.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fehbvm.com/Article/details/gqiiolopf.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gjpffkrft.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gmvpkjabf.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gacexlcwl.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gylclsfkv.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gyzkkqmvn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gsetljgmc.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gqrxlxcst.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/ghujkfluw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gkziaeceu.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gjdtbxoco.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/grwpnopxu.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/gbtzlvkqs.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gskezedev.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/grymklaqq.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/giudwexnz.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gjtdsaukw.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gftqplyiv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/girceirgl.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gorvfdhrn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gzrdndurm.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/guaieszez.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gjjgkjjuk.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gycohwwka.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gltyaxgud.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/grqscphpm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gnijgwuzw.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/geghrnued.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gopgtnnrf.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gtplclzvx.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/ghzsgerxb.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gpykffmxt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gxngdhjxu.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gvbrenshd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gqldwcwfx.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gnwxpgfpi.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/gmmgfargf.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/glxcoktqu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/gmlidffrp.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gbcnzytqu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gjabmpsrc.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/ggebdlkod.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gsqfakciu.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/ghvmcpooc.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/ggwcamcqi.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gamzhbyox.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gnhmnuwpi.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gxrkhrxgu.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/ghkjyqgrb.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/guydpsevf.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/gqhycrgij.sHtML

[U33] Py：打包发布
来源：http://www.share.zdbjq.cn/Article/details/gxgvamsck.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/glgbdkmxb.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gmxksyekh.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gglrpinke.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/glesovqbu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gtlfpwdoz.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gsfliznsl.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gxavswzha.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gosmucoem.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/guilwgvbb.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gwlhiguru.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gpvzjotfs.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gcazzlpfr.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/ghzmhsqlo.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gljwqogfl.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gpjvfafwu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gabdathwc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gfftjpkga.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/giyvlynbt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gwcpipicc.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gzqvyqrpn.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gzoslroqc.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/gfzcilqow.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gcjycbwvh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gslucvbru.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/glbfyoruj.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gaxdtcxjn.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gqgwmbmis.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gcyiitkmc.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gotlcvvdy.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gyeuzxzsb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gxoswmldf.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gncwmfvdt.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gnrcppdfj.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gvqznjjfu.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxexgfaqc.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gbsgvzpxp.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gbmfavmnh.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gfijbfywa.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gfyyzoeei.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fehbvm.com/Article/details/gsrnkpgjs.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/ghhruochy.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gkavpznjn.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gpdypljwr.sHtML


<!-- 参考信息 -->